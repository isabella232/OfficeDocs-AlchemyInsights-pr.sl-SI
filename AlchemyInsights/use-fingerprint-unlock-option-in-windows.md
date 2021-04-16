---
title: Možnost odklepanja prstnih odtisov v sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796693"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="43da8-102">Možnost odklepanja prstnih odtisov v sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="43da8-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="43da8-103">**Omogočanje prstnih odtisov s funkcijo Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="43da8-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="43da8-104">Če želite odkleniti sistem Windows 10 s prstnim odtisom, morate nastaviti prstni odtis Windows Hello tako, da dodate vsaj en prst (tako da sistem Windows prepozna).</span><span class="sxs-lookup"><span data-stu-id="43da8-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="43da8-105">Pojdite na **Nastavitve > Računi > možnosti vpisa** (ali kliknite [tukaj](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="43da8-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="43da8-106">Na seznamu bodo navedene razpoložljive možnosti za vpis.</span><span class="sxs-lookup"><span data-stu-id="43da8-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="43da8-107">Na primer:</span><span class="sxs-lookup"><span data-stu-id="43da8-107">For example:</span></span>

    ![Možnosti vpisa.](media/sign-in-options.png)

2. <span data-ttu-id="43da8-109">Kliknite ali tapnite **Windows Hello prstni** odtis , nato pa kliknite **Nastavitev**.</span><span class="sxs-lookup"><span data-stu-id="43da8-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="43da8-110">V oknu za namestitev Windows Hello kliknite **Uvod.**</span><span class="sxs-lookup"><span data-stu-id="43da8-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="43da8-111">Senzor prstnih odtisov se bo aktiviral in pozvani boste, da postavite prst na senzor:</span><span class="sxs-lookup"><span data-stu-id="43da8-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Senzor prstnih odtisov.](media/fingerprint-sensor.png)

3. <span data-ttu-id="43da8-113">Upoštevajte navodila, ki vas bodo pozvala, da večkrat pregledate prst.</span><span class="sxs-lookup"><span data-stu-id="43da8-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="43da8-114">Ko bo ta rešitev končana, lahko dodate druge prste, ki jih boste morda želeli uporabiti za vpis.</span><span class="sxs-lookup"><span data-stu-id="43da8-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="43da8-115">Ko se boste naslednjič vpisati v Windows 10, boste imeli možnost, da za to uporabite svoj prstni odtis.</span><span class="sxs-lookup"><span data-stu-id="43da8-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="43da8-116">**Možnost za vpis s prstnim odtisom Windows Hello ni na voljo**</span><span class="sxs-lookup"><span data-stu-id="43da8-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="43da8-117">Če možnost Prstni odtis Windows Hello ni prikazana kot možnost v možnostih vpisa, sistem Windows ne pozna bralnika prstnih odtisov/optičnega bralnika, ki je priključen na računalnik, ali da sistemski pravilnik preprečuje njegovo uporabo (če na primer vaš računalnik upravlja vaše delovno mesto).</span><span class="sxs-lookup"><span data-stu-id="43da8-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="43da8-118">Odpravljanje težav:</span><span class="sxs-lookup"><span data-stu-id="43da8-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="43da8-119">Izberite gumb **za začetni** meni v opravilni vrstici in poiščite **Upravitelja naprav**.</span><span class="sxs-lookup"><span data-stu-id="43da8-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="43da8-120">Kliknite ali tapnite, da odprete **upravitelja naprav.**</span><span class="sxs-lookup"><span data-stu-id="43da8-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="43da8-121">V upravitelju naprav razširite biometrične naprave tako, da kliknete škarne.</span><span class="sxs-lookup"><span data-stu-id="43da8-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrične naprave.](media/biometric-devices.png)

4. <span data-ttu-id="43da8-123">Optični bralnik za prstni odtis mora biti naveden kot biometrična naprava, kot je optični bralnik Synaptics WBDI:</span><span class="sxs-lookup"><span data-stu-id="43da8-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrične naprave.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="43da8-125">Če bralnik prstnih odtisov ni prikazan in je optični bralnik integriran z vašim računalnikom, obiščite spletno mesto izdelovalca računalnika.</span><span class="sxs-lookup"><span data-stu-id="43da8-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="43da8-126">V razdelku za tehnično podporo za svoj model računalnika poiščite gonilnik sistema Windows 10, da poiščete optični bralnik, ki ga lahko namestite.</span><span class="sxs-lookup"><span data-stu-id="43da8-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="43da8-127">Če je optični bralnik ločen od računalnika (priključen prek USB-ja), obiščite spletno mesto izdelovalca optičnega bralnika in poiščite ter namestite programsko opremo gonilnika naprave s sistemom Windows 10 za model optičnega bralnika, ki ga imate.</span><span class="sxs-lookup"><span data-stu-id="43da8-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
