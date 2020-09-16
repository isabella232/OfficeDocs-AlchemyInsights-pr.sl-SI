---
title: Vpis v Windows 10 brez gesla
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
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719969"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="936cb-102">Vpis v Windows 10 brez gesla</span><span class="sxs-lookup"><span data-stu-id="936cb-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="936cb-103">Če se želite izogniti vnosu gesla pri zagonu sistema Windows, vam priporočamo, da uporabite eno od varnih možnosti za vpis v sistemu Windows, na primer PIN, prepoznavanje obrazov ali prstni odtis, če je na voljo.</span><span class="sxs-lookup"><span data-stu-id="936cb-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="936cb-104">Če želite onemogočiti varno prijavo, si oglejte spodnja navodila» samodejno vpis v Windows 10 «.</span><span class="sxs-lookup"><span data-stu-id="936cb-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="936cb-105">**Varni Windows hello alternative geslom za račun**</span><span class="sxs-lookup"><span data-stu-id="936cb-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="936cb-106">Pojdite na **nastavitve > računov > možnosti za vpis** (ali kliknite [tukaj](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="936cb-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="936cb-107">Na voljo bodo navedene možnosti za vpis.</span><span class="sxs-lookup"><span data-stu-id="936cb-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="936cb-108">Na primer:</span><span class="sxs-lookup"><span data-stu-id="936cb-108">For example:</span></span>

![Možnosti vpisa.](media/sign-in-options.png)

<span data-ttu-id="936cb-110">Kliknite ali tapnite eno od možnosti, da jo konfigurirate.</span><span class="sxs-lookup"><span data-stu-id="936cb-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="936cb-111">Ko boste naslednjič zagnali ali odklenili sistem Windows, boste lahko namesto gesla uporabili novo možnost.</span><span class="sxs-lookup"><span data-stu-id="936cb-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="936cb-112">**Samodejno vpis v Windows 10**</span><span class="sxs-lookup"><span data-stu-id="936cb-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="936cb-113">**Opomba**: samodejno vpis je priročno, vendar uvaja varnostno tveganje, še posebej, če je vaš računalnik dostopen z več osebami.</span><span class="sxs-lookup"><span data-stu-id="936cb-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="936cb-114">Kliknite ali tapnite gumb **Start** v opravilni vrstici.</span><span class="sxs-lookup"><span data-stu-id="936cb-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="936cb-115">Vnesite **netplwiz** in pritisnite tipko ENTER, da odprete okno uporabniških računov.</span><span class="sxs-lookup"><span data-stu-id="936cb-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="936cb-116">V **uporabniških računih**kliknite račun, s katerim se želite samodejno vpisati, ko se Windows zažene.</span><span class="sxs-lookup"><span data-stu-id="936cb-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="936cb-117">Počistite potrditveno polje» Uporabniki morajo vnesti uporabniško ime in geslo za uporabo tega računalnika «.</span><span class="sxs-lookup"><span data-stu-id="936cb-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Uporabniki morajo vnesti možnost uporabniškega imena in gesla.](media/users-must-enter-username.png)

5. <span data-ttu-id="936cb-119">Kliknite **V redu**.</span><span class="sxs-lookup"><span data-stu-id="936cb-119">Click **OK**.</span></span> <span data-ttu-id="936cb-120">Pozvani boste k vnosu in potrditvi gesla za račun, ki ste ga izbrali.</span><span class="sxs-lookup"><span data-stu-id="936cb-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="936cb-121">Kliknite **v redu** , da dokončujete.</span><span class="sxs-lookup"><span data-stu-id="936cb-121">Click **OK** to finish.</span></span> <span data-ttu-id="936cb-122">Naslednjič, ko se zažene Windows 10, se bo samodejno vpisal v račun, ki ste ga izbrali.</span><span class="sxs-lookup"><span data-stu-id="936cb-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
