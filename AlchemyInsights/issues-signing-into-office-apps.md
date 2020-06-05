---
title: Težave pri vpisu v Microsoft 365 apps
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
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579881"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="acf7d-102">Popravljanje Microsoftovih 365 aplikacij» modul zaupanja vrednih platform računalnika ne deluje pravilno «</span><span class="sxs-lookup"><span data-stu-id="acf7d-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="acf7d-103">Če želite to napako odpraviti, poskusite to:</span><span class="sxs-lookup"><span data-stu-id="acf7d-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="acf7d-104">Namestite najnovejše posodobitve za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) in [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="acf7d-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="acf7d-105">[Počistite Officeove poverilnice](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic Windows.</span><span class="sxs-lookup"><span data-stu-id="acf7d-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="acf7d-106">**Opomba:** Registrske poti za Office 2016 so se spremenile v 16,0.</span><span class="sxs-lookup"><span data-stu-id="acf7d-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="acf7d-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="acf7d-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="acf7d-108">Preizkusite [postopek za obnovitev uporabnika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) , da odpravite napake modula zaupanja vrednih platform (TPM).</span><span class="sxs-lookup"><span data-stu-id="acf7d-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="acf7d-109">Nastavite EnableADAL = 0 z naslednjimi koraki:</span><span class="sxs-lookup"><span data-stu-id="acf7d-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="acf7d-110">Z desno tipko miške kliknite gumb Start sistema Windows, izberite **Zaženi**, vnesite **regedit**in izberite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="acf7d-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="acf7d-111">Izberite **da** , če želite urejevalniku registra omogočiti spreminjanje naprave.</span><span class="sxs-lookup"><span data-stu-id="acf7d-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="acf7d-112">V urejevalniku registra dodajte vrednost DWORD **Enableadal** z nastavitvijo **0** pod HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="acf7d-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="acf7d-113">Če želite več informacij, glejte [težave s povezavo v vpisu po posodobitvi v Office 2016 graditi 16.0.7967 v operacijskem sistemu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="acf7d-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>