---
title: Težave pri vpisu v programe Microsoft 365
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
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709122"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="696f5-102">Popravljanje aplikacije Microsoft 365 apps» modul zaupanja vredne platforme računalnika ni pravilno delujoč «</span><span class="sxs-lookup"><span data-stu-id="696f5-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="696f5-103">Če želite to napako odpraviti, poskusite to:</span><span class="sxs-lookup"><span data-stu-id="696f5-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="696f5-104">Namestite najnovejše posodobitve za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) in [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="696f5-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="696f5-105">[Počistite Officeove poverilnice](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic sistema Windows.</span><span class="sxs-lookup"><span data-stu-id="696f5-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="696f5-106">**Opomba:** Poti registra za Office 2016 so se spremenile v 16,0.</span><span class="sxs-lookup"><span data-stu-id="696f5-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="696f5-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="696f5-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="696f5-108">Preskusite [postopek za obnovitev uporabnika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) , da odpravite napake modula zaupanja TPM.</span><span class="sxs-lookup"><span data-stu-id="696f5-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="696f5-109">Nastavite EnableADAL = 0 s temi koraki:</span><span class="sxs-lookup"><span data-stu-id="696f5-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="696f5-110">Z desno tipko miške kliknite gumb Start sistema Windows, izberite **Zaženi**, vnesite **regedit** in nato izberite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="696f5-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="696f5-111">Izberite **da** , da omogočite urejevalnik registra, da spremenite vašo napravo.</span><span class="sxs-lookup"><span data-stu-id="696f5-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="696f5-112">V urejevalniku registra dodajte vrednost DWORD **EnableADAL** z nastavitvami **0** v razdelku HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="696f5-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="696f5-113">Če želite več informacij, glejte [težave s povezavo v vpisu po posodobitvi na Office 2016 Build 16.0.7967 v sistemu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="696f5-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>