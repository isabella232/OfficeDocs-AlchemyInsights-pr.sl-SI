---
title: Vpis v Windows 10 brez gesla
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
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830562"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="3316e-102">Vpis v Windows 10 brez gesla</span><span class="sxs-lookup"><span data-stu-id="3316e-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="3316e-103">Če se želite izogniti vnosu gesla ob zagonu sistema Windows, priporočamo, da uporabite eno od možnosti varnega vpisa s funkcijo Windows Hello, kot je KODA PIN, prepoznavanje obraza ali prstni odtis, če je na voljo.</span><span class="sxs-lookup"><span data-stu-id="3316e-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="3316e-104">Če res želite onemogočiti varni vpis, preberite spodnja navodila »Samodejni vpis v Windows 10«.</span><span class="sxs-lookup"><span data-stu-id="3316e-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="3316e-105">**Zaščitite nadomestne možnosti za Windows Hello za geslo računa**</span><span class="sxs-lookup"><span data-stu-id="3316e-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="3316e-106">Pojdite na **Nastavitve > Računi > možnosti vpisa** (ali kliknite [tukaj](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="3316e-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="3316e-107">Na seznamu bodo navedene razpoložljive možnosti za vpis.</span><span class="sxs-lookup"><span data-stu-id="3316e-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="3316e-108">Na primer:</span><span class="sxs-lookup"><span data-stu-id="3316e-108">For example:</span></span>

![Možnosti vpisa.](media/sign-in-options.png)

<span data-ttu-id="3316e-110">Kliknite ali tapnite eno od možnosti, da jo konfigurirate.</span><span class="sxs-lookup"><span data-stu-id="3316e-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="3316e-111">Ob naslednjem zagonu ali odklepanju sistema Windows boste lahko namesto gesla uporabili novo možnost.</span><span class="sxs-lookup"><span data-stu-id="3316e-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="3316e-112">**Samodejni vpis v Windows 10**</span><span class="sxs-lookup"><span data-stu-id="3316e-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="3316e-113">**Opomba:** Samodejni vpis je priročen, vendar predstavlja varnostno tveganje, še posebej, če je vaš računalnik dostopen več ljudem.</span><span class="sxs-lookup"><span data-stu-id="3316e-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="3316e-114">Kliknite ali tapnite gumb **za začetni meni** v opravilni vrstici.</span><span class="sxs-lookup"><span data-stu-id="3316e-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="3316e-115">Vnesite **netplwiz in pritisnite** tipko Enter, da odprete okno Uporabniški računi.</span><span class="sxs-lookup"><span data-stu-id="3316e-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="3316e-116">V **oknu Uporabniški** računi kliknite račun, v katerega se želite samodejno vpisati ob zagonu sistema Windows.</span><span class="sxs-lookup"><span data-stu-id="3316e-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="3316e-117">Počistite potrditveno polje »Uporabniki morajo vnesti uporabniško ime in geslo, če morajo uporabljati ta računalnik«.</span><span class="sxs-lookup"><span data-stu-id="3316e-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Uporabniki morajo vnesti uporabniško ime in možnost gesla.](media/users-must-enter-username.png)

5. <span data-ttu-id="3316e-119">Kliknite **V redu**.</span><span class="sxs-lookup"><span data-stu-id="3316e-119">Click **OK**.</span></span> <span data-ttu-id="3316e-120">Pozvani boste k vnosu in potrditvi gesla za izbrani račun.</span><span class="sxs-lookup"><span data-stu-id="3316e-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="3316e-121">Če želite **končati,** kliknite V redu.</span><span class="sxs-lookup"><span data-stu-id="3316e-121">Click **OK** to finish.</span></span> <span data-ttu-id="3316e-122">Ob naslednjem zagonu sistema Windows 10 se samodejno vpiše v račun, ki ste ga izbrali.</span><span class="sxs-lookup"><span data-stu-id="3316e-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
