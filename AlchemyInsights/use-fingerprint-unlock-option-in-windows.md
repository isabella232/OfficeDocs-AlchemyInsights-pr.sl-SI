---
title: Uporaba možnosti odklepanja prstnih odtisov v sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588331"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="7998f-102">Uporaba možnosti odklepanja prstnih odtisov v sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="7998f-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="7998f-103">**Omogoči Windows hello prstni odtis**</span><span class="sxs-lookup"><span data-stu-id="7998f-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="7998f-104">Če želite odkleniti sistem Windows 10 s prstnim odtisom, morate nastaviti Windows hello prstni odtis tako, da dodate (dovolite, da se Windows nauči prepoznati) vsaj en prst.</span><span class="sxs-lookup"><span data-stu-id="7998f-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="7998f-105">Odprite **možnost nastavitve > računi > možnosti prijave** (ali kliknite [tukaj](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="7998f-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="7998f-106">Navedene bodo razpoložljive možnosti za vpis.</span><span class="sxs-lookup"><span data-stu-id="7998f-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="7998f-107">Na primer:</span><span class="sxs-lookup"><span data-stu-id="7998f-107">For example:</span></span>

    ![Možnosti vpisnega znaka.](media/sign-in-options.png)

2. <span data-ttu-id="7998f-109">Kliknite ali tapnite **Windows hello prstni odtis**, nato pa kliknite **Nastavi**.</span><span class="sxs-lookup"><span data-stu-id="7998f-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="7998f-110">V oknu z nastavitvami sistema Windows hello kliknite **Začni**.</span><span class="sxs-lookup"><span data-stu-id="7998f-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="7998f-111">Senzor prstnih odtisov bo aktiviran in pozvani boste, da Položite prst na senzor:</span><span class="sxs-lookup"><span data-stu-id="7998f-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Senzor prstnih odtisov.](media/fingerprint-sensor.png)

3. <span data-ttu-id="7998f-113">Upoštevajte navodila, ki vas bodo prosila, da večkrat skenirate prst.</span><span class="sxs-lookup"><span data-stu-id="7998f-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="7998f-114">Ko končate, boste imeli možnost dodajanja drugih prstov, ki jih boste morda želeli uporabiti za vpis.</span><span class="sxs-lookup"><span data-stu-id="7998f-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="7998f-115">Ko se boste naslednjič prijavili v sistem Windows 10, boste imeli možnost, da to storite s prstnim odtisom.</span><span class="sxs-lookup"><span data-stu-id="7998f-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="7998f-116">**Windows hello prstni odtis ni na voljo kot možnost prijave**</span><span class="sxs-lookup"><span data-stu-id="7998f-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="7998f-117">Če Windows hello prstni odtis ni prikazan kot možnost v **možnosti prijave**, to pomeni, da Windows ne pozna nobenega bralnika prstnih odtisov/skenerja, priloženega računalniku, ali da sistemska politika preprečuje njegovo uporabo (če na primer vaš računalnik upravlja vaše delovno mesto).</span><span class="sxs-lookup"><span data-stu-id="7998f-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="7998f-118">Za odpravljanje težav:</span><span class="sxs-lookup"><span data-stu-id="7998f-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="7998f-119">V opravilni vrstici izberite gumb **Start** in poiščite **upravitelja naprav**.</span><span class="sxs-lookup"><span data-stu-id="7998f-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="7998f-120">Kliknite ali tapnite, da odprete **upravitelja naprav**.</span><span class="sxs-lookup"><span data-stu-id="7998f-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="7998f-121">V upravitelju naprav razširite biometrične naprave tako, da kliknete njegov Chevron.</span><span class="sxs-lookup"><span data-stu-id="7998f-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrične naprave.](media/biometric-devices.png)

4. <span data-ttu-id="7998f-123">Optični bralnik prstnih odtisov mora biti naveden kot biometrična naprava, kot je optični bralnik Synaptics WBDI:</span><span class="sxs-lookup"><span data-stu-id="7998f-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrične naprave.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="7998f-125">Če optični bralnik prstnih odtisov ni prikazan in je optični bralnik vgrajen v računalnik, obiščite spletno mesto izdelovalca računalnika.</span><span class="sxs-lookup"><span data-stu-id="7998f-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="7998f-126">V razdelku za tehnično podporo za model računalnika poiščite gonilnik za Windows 10 za skener, ki ga lahko namestite.</span><span class="sxs-lookup"><span data-stu-id="7998f-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="7998f-127">Če je optični bralnik ločen od računalnika (priložen prek USB-ja), obiščite spletno mesto izdelovalca optičnega bralnika, da poiščete in namestite programsko opremo gonilnika naprave Windows 10 za model optičnega bralnika, ki ga imate.</span><span class="sxs-lookup"><span data-stu-id="7998f-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
