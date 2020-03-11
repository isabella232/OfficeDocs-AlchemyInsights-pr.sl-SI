---
title: Vpis v sistem Windows 10 brez uporabe gesla
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588296"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="04708-102">Vpis v sistem Windows 10 brez uporabe gesla</span><span class="sxs-lookup"><span data-stu-id="04708-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="04708-103">Če se želite izogniti temu, da bi morali vnesti geslo ob zagonu sistema Windows, priporočamo, da uporabite eno od možnosti varne prijave v sistemu Windows hello, na primer kodo PIN, prepoznavanje obrazov ali prstni odtis, če je na voljo.</span><span class="sxs-lookup"><span data-stu-id="04708-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="04708-104">Če res želite onemogočiti varno prijavo, glejte spodnja navodila» samodejno vpis v sistem Windows 10 «.</span><span class="sxs-lookup"><span data-stu-id="04708-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="04708-105">**Varno Windows hello alternative geslo za račun**</span><span class="sxs-lookup"><span data-stu-id="04708-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="04708-106">Odprite **možnost nastavitve > računi > možnosti prijave** (ali kliknite [tukaj](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="04708-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="04708-107">Navedene bodo razpoložljive možnosti za vpis.</span><span class="sxs-lookup"><span data-stu-id="04708-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="04708-108">Na primer:</span><span class="sxs-lookup"><span data-stu-id="04708-108">For example:</span></span>

![Možnosti vpisnega znaka.](media/sign-in-options.png)

<span data-ttu-id="04708-110">Kliknite ali tapnite eno od možnosti, da jo konfigurirate.</span><span class="sxs-lookup"><span data-stu-id="04708-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="04708-111">Ko naslednjič zaženete ali odklenete sistem Windows, boste lahko namesto gesla uporabili novo možnost.</span><span class="sxs-lookup"><span data-stu-id="04708-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="04708-112">**Samodejno vpis v sistem Windows 10**</span><span class="sxs-lookup"><span data-stu-id="04708-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="04708-113">**Opomba**: Samodejna prijava je priročna, vendar uvaja varnostno tveganje, še posebej, če je računalnik dostopen več osebam.</span><span class="sxs-lookup"><span data-stu-id="04708-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="04708-114">Kliknite ali tapnite gumb **Start** v opravilni vrstici.</span><span class="sxs-lookup"><span data-stu-id="04708-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="04708-115">Stavek **netplwiz** ter zadeti nastopiti zakleniti razkleniti uporabnik račun okno.</span><span class="sxs-lookup"><span data-stu-id="04708-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="04708-116">V **uporabniških računih**kliknite račun, v katerega se želite samodejno vpisati, ko se Windows zažene.</span><span class="sxs-lookup"><span data-stu-id="04708-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="04708-117">Nenadzirljiv "uporabnik morati nastopiti a uporabnik ime ter parola rabiti to računalo" čekovna knjižica.</span><span class="sxs-lookup"><span data-stu-id="04708-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Uporabnik morati nastopiti a username ter parola predkupna pravica.](media/users-must-enter-username.png)

5. <span data-ttu-id="04708-119">Kliknite **V redu**.</span><span class="sxs-lookup"><span data-stu-id="04708-119">Click **OK**.</span></span> <span data-ttu-id="04708-120">Pozvani boste, da vnesete in potrdite geslo za izbrani račun.</span><span class="sxs-lookup"><span data-stu-id="04708-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="04708-121">Kliknite **v redu** , da končate.</span><span class="sxs-lookup"><span data-stu-id="04708-121">Click **OK** to finish.</span></span> <span data-ttu-id="04708-122">Naslednjič, ko se Windows 10 zažene, se bo samodejno vpisalo v izbrani račun.</span><span class="sxs-lookup"><span data-stu-id="04708-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
