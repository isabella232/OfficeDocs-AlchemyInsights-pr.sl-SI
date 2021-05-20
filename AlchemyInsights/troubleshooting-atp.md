---
title: Odpravljanje težav s programom Microsoft Defender Office 365
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
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545284"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="81ef3-102">Odpravljanje težav s programom Microsoft Defender Office 365</span><span class="sxs-lookup"><span data-stu-id="81ef3-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="81ef3-103">**Ali opazite zakasnitve pri dostavi sporočila?**</span><span class="sxs-lookup"><span data-stu-id="81ef3-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="81ef3-104">Uporabite možnost [dinamične dostave](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) v pravilniku microsoft Defender za Office 365 Sef prilog.</span><span class="sxs-lookup"><span data-stu-id="81ef3-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="81ef3-105">Tako boste preprečili zakasnitve sporočil in pri tem zaščitili prejemnike pred zlonamernimi datotekami.</span><span class="sxs-lookup"><span data-stu-id="81ef3-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="81ef3-106">**Ali želite Microsoftu prijaviti napačne pozitivne ali napačne negativne vrednosti?**</span><span class="sxs-lookup"><span data-stu-id="81ef3-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="81ef3-107">Uporabite [Raziskovalca za pošiljanje.](https://protection.office.com/reportsubmission)</span><span class="sxs-lookup"><span data-stu-id="81ef3-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="81ef3-108">-\*\* Ali ste vedeli, da lahko omogočite zaščito Sef povezave za notranjo e-pošto, poslano med prejemniki v organizaciji?\*\* Upoštevajte ta navodila:</span><span class="sxs-lookup"><span data-stu-id="81ef3-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="81ef3-109">Pojdite v [https://protection.office.com](https://protection.office.com) račun globalnega skrbnika ali skrbnika za varnost in se vpišite z njim.</span><span class="sxs-lookup"><span data-stu-id="81ef3-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="81ef3-110">V levem podoknu za krmarjenje **v razdelku Upravljanje groženj** izberite **Povezave** \> **Sef pravilnika.**</span><span class="sxs-lookup"><span data-stu-id="81ef3-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="81ef3-111">V razdelku **Pravilniki, ki veljajo za celotno organizacijo** izberite pravilnik in kliknite **Uredi**.</span><span class="sxs-lookup"><span data-stu-id="81ef3-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="81ef3-112">V **Nastavitve**, omogočite **Uporabi varne povezave za sporočila, poslana znotraj organizacije.**</span><span class="sxs-lookup"><span data-stu-id="81ef3-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
