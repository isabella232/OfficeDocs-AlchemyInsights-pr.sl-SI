---
title: Težave pri vpisu v aplikacije Microsoft 365
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
- "9000571"
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833031"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="94e15-102">Sporočilo o odpravljanju težav v aplikacijah Microsoft 365 »Modul zaupanja vredne platforme vašega računalnika ne deluje pravilno«</span><span class="sxs-lookup"><span data-stu-id="94e15-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="94e15-103">Če želite to napako odpraviti, poskusite to:</span><span class="sxs-lookup"><span data-stu-id="94e15-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="94e15-104">Namestite najnovejše posodobitve za [Windows in](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="94e15-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="94e15-105">[Počistite poverilnice za Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic sistema Windows.</span><span class="sxs-lookup"><span data-stu-id="94e15-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="94e15-106">**Opomba:** Poti registra za Office 2016 so se spremenile v 16.0.</span><span class="sxs-lookup"><span data-stu-id="94e15-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="94e15-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="94e15-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="94e15-108">Poskusite postopek [obnovitve uporabnika, da](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) odpravite napake modula zaupanja vrednih platform (TPM).</span><span class="sxs-lookup"><span data-stu-id="94e15-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="94e15-109">Nastavite EnableADAL = 0 tako, da sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="94e15-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="94e15-110">Z desno tipko miške kliknite gumb Start sistema Windows, **izberite Zaženi**, vnesite **regedit** in nato izberite V **redu**.</span><span class="sxs-lookup"><span data-stu-id="94e15-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="94e15-111">Če **želite** urejevalniku registra dovoliti spreminjanje naprave, izberite Da.</span><span class="sxs-lookup"><span data-stu-id="94e15-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="94e15-112">V urejevalniku registra dodajte vrednost DWORD za **EnableADAL** z nastavitvijo **0** v razdelku HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="94e15-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="94e15-113">Če želite več informacij, glejte Težave pri vpisu s povezavo po posodobitvi na [gradovi Office 2016, graden 16.0.7967 v sistemu Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="94e15-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>