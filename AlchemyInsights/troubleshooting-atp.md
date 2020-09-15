---
title: Odpravljanje težav z zaščito pred grožnjami sistema Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 5a13653ba08d8c6b822354ff70f6d276d31cd816
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658930"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="f8365-102">Odpravljanje težav z zaščito pred grožnjami sistema Office 365</span><span class="sxs-lookup"><span data-stu-id="f8365-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="f8365-103">Ali opazite zamude pri dostavi sporočila?</span><span class="sxs-lookup"><span data-stu-id="f8365-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="f8365-104">Uporabite možnost [dinamična dostava](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) v pravilniku o varnih prilogah za ATP.</span><span class="sxs-lookup"><span data-stu-id="f8365-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="f8365-105">S tem se izognete zakasnitvam sporočil in zaščitite prejemnike pred zlonamernimi datotekami.</span><span class="sxs-lookup"><span data-stu-id="f8365-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="f8365-106">Ali želite Microsoftu prijaviti lažne pozitivne ali lažne negativne izraze?</span><span class="sxs-lookup"><span data-stu-id="f8365-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="f8365-107">S to [povezavo](https://www.microsoft.com/wdsi/filesubmission/) lahko pošljete datoteke v analizo.</span><span class="sxs-lookup"><span data-stu-id="f8365-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="f8365-108">Ali ste vedeli, da lahko omogočite zaščito varnih povezav za notranjo e-pošto, poslano med prejemniki v organizaciji?</span><span class="sxs-lookup"><span data-stu-id="f8365-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="f8365-109">Upoštevajte te korake:</span><span class="sxs-lookup"><span data-stu-id="f8365-109">Follow these steps:</span></span>

  1. <span data-ttu-id="f8365-110">Pojdite na [https://protection.office.com](https://protection.office.com) in se vpišite z računom globalnega skrbnika ali varnostnega skrbnika.</span><span class="sxs-lookup"><span data-stu-id="f8365-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="f8365-111">V levem podoknu za krmarjenje v razdelku **upravljanje groženj**izberite povezave **pravilnika** za \> **varnost**.</span><span class="sxs-lookup"><span data-stu-id="f8365-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="f8365-112">V razdelku **pravilniki, ki veljajo za celotno organizacijo** , izberite pravilnik in kliknite **Uredi**.</span><span class="sxs-lookup"><span data-stu-id="f8365-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="f8365-113">V razdelku **Nastavitve**omogočite **Uporaba varnih povezav do sporočil, poslanih v organizaciji**.</span><span class="sxs-lookup"><span data-stu-id="f8365-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
