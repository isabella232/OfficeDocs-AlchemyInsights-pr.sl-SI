---
title: Uporaba možnosti odklepanja prstnih odtisov v sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795260"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="0301b-102">Uporaba možnosti odklepanja prstnih odtisov v sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="0301b-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="0301b-103">**Omogočanje pozdravnega prstnega odtisa sistema Windows**</span><span class="sxs-lookup"><span data-stu-id="0301b-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="0301b-104">Če želite odkleniti Windows 10 s prstnim odtisom, morate nastaviti pozdravni prstni odtis sistema Windows, tako da dodate (oddajanje sistema Windows se naučite prepoznati) vsaj en prst.</span><span class="sxs-lookup"><span data-stu-id="0301b-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="0301b-105">Pojdite na **nastavitve > računov > možnosti za vpis** (ali kliknite [tukaj](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="0301b-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="0301b-106">Na voljo bodo navedene možnosti za vpis.</span><span class="sxs-lookup"><span data-stu-id="0301b-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="0301b-107">Na primer:</span><span class="sxs-lookup"><span data-stu-id="0301b-107">For example:</span></span>

    ![Možnosti vpisa.](media/sign-in-options.png)

2. <span data-ttu-id="0301b-109">Kliknite ali tapnite **Pozdravni prstni odtis sistema Windows**, nato pa kliknite **Nastavi**.</span><span class="sxs-lookup"><span data-stu-id="0301b-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="0301b-110">V oknu Windows hello **setup kliknite Začni**.</span><span class="sxs-lookup"><span data-stu-id="0301b-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="0301b-111">Senzor prstnih odtisov bo aktiviran in pozvani boste, da postavite kazalec na tipalo:</span><span class="sxs-lookup"><span data-stu-id="0301b-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Senzor prstnih odtisov.](media/fingerprint-sensor.png)

3. <span data-ttu-id="0301b-113">Sledite navodilom, ki vas bodo pozvali, da večkrat skenirate prst.</span><span class="sxs-lookup"><span data-stu-id="0301b-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="0301b-114">Ko je ta možnost končana, boste lahko dodali še druge prste, ki jih boste morda želeli uporabiti za vpis.</span><span class="sxs-lookup"><span data-stu-id="0301b-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="0301b-115">Ko se naslednjič vpišete v sistem Windows 10, boste imeli na voljo možnost uporabe prstnega odtisa.</span><span class="sxs-lookup"><span data-stu-id="0301b-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="0301b-116">**Pozdravni prstni odtis sistema Windows ni na voljo kot možnost za vpis**</span><span class="sxs-lookup"><span data-stu-id="0301b-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="0301b-117">Če se prstni odtis sistema Windows ne prikaže kot možnost v **možnostih za vpis**, to pomeni, da Windows ne pozna nobenega bralnika prstnih odtisov ali skenerja, ki je priključen na vaš računalnik, ali da sistemska politika preprečuje njegovo uporabo (če je na primer vaš računalnik upravljan na delovnem mestu).</span><span class="sxs-lookup"><span data-stu-id="0301b-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="0301b-118">Odpravljanje težav:</span><span class="sxs-lookup"><span data-stu-id="0301b-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="0301b-119">V opravilni vrstici izberite gumb **Start** in poiščite **upravitelja naprav**.</span><span class="sxs-lookup"><span data-stu-id="0301b-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="0301b-120">Kliknite ali tapnite, da odprete **upravitelja naprav**.</span><span class="sxs-lookup"><span data-stu-id="0301b-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="0301b-121">V upravitelju naprav razširite biometrične naprave tako, da kliknete njen Chevron.</span><span class="sxs-lookup"><span data-stu-id="0301b-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrične naprave.](media/biometric-devices.png)

4. <span data-ttu-id="0301b-123">Bralnik prstnih odtisov bi moral biti naveden kot biometrična naprava, kot je na primer Synaptics WBDI Scanner:</span><span class="sxs-lookup"><span data-stu-id="0301b-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrične naprave.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="0301b-125">Če skenerja prstnih odtisov ni prikazan in je optični bralnik vdelan v računalnik, obiščite spletno mesto izdelovalca računalnika.</span><span class="sxs-lookup"><span data-stu-id="0301b-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="0301b-126">V razdelku tehnična podpora za model računalnika poiščite gonilnik sistema Windows 10 za skener, ki ga lahko namestite.</span><span class="sxs-lookup"><span data-stu-id="0301b-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="0301b-127">Če je optični bralnik ločen od računalnika (priloženo prek USB-ja), obiščite spletno mesto izdelovalca optičnega bralnika, da poiščete in namestite programsko opremo gonilnika naprave Windows 10 za model skenerja, ki ga imate.</span><span class="sxs-lookup"><span data-stu-id="0301b-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
