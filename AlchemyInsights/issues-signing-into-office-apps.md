---
title: Vprašanja, ki se vpisujete Office aplikacije
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938344"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="c40ed-102">Določitev urad apps "modula zaupanja TPM računalnika ne deluje pravilno" sporočilo</span><span class="sxs-lookup"><span data-stu-id="c40ed-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="c40ed-103">Če želite odpraviti to napako, poskusite naslednje:</span><span class="sxs-lookup"><span data-stu-id="c40ed-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="c40ed-104">Namestite najnovejše posodobitve za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) in [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="c40ed-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="c40ed-105">[Jasno urad poverilnic](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic Windows.</span><span class="sxs-lookup"><span data-stu-id="c40ed-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="c40ed-106">**Opomba:** Registrske poti za Office 2016 spremenili v 16,0.</span><span class="sxs-lookup"><span data-stu-id="c40ed-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="c40ed-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="c40ed-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="c40ed-108">Začeti [postopek izterjave uporabnik](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) popraviti napake Modul TPM (Trusted Platform).</span><span class="sxs-lookup"><span data-stu-id="c40ed-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="c40ed-109">Nastaviti v EnableADAL = 0, po naslednjih korakih:</span><span class="sxs-lookup"><span data-stu-id="c40ed-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="c40ed-110">Z desno tipko miške na gumb Start, izberite **Zaženi**, vnesite **regedit**in izberite **OK**.</span><span class="sxs-lookup"><span data-stu-id="c40ed-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="c40ed-111">Izberite **ja** omogočiti urejevalnik registra, da spremenite napravo.</span><span class="sxs-lookup"><span data-stu-id="c40ed-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="c40ed-112">V registracija urednik, dodajte vrednost DWORD **EnableADAL** s nastavitev **0** pod HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="c40ed-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="c40ed-113">Če želite več informacij, glejte [te¾ave pri povezovanju v vpisno po posodobitvi za Office 2016 zidava 16.0.7967 na Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="c40ed-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>