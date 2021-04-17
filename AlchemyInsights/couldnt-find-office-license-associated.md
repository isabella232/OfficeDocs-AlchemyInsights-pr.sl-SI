---
title: Popravljanje sporočil, da v aplikacijah Microsoft 365 ni bilo mogoče najti licenc za Office
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
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816504"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="77da5-102">Popravljanje sporočila »Povezanih officeovih licenc ni bilo mogoče najti« v aplikacijah Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="77da5-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="77da5-103">Če se prikaže to sporočilo, poskusite to:</span><span class="sxs-lookup"><span data-stu-id="77da5-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="77da5-104">Preverite nastavitve požarnega zidu, protivirusne programske opreme in strežnika proxy, da potrdite, da ne blokirajo dostopa do interneta do aplikacij storitve Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="77da5-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="77da5-105">Glejte [URL-ji in obsegi naslovov IP za Microsoft 365.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="77da5-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="77da5-106">Odstranite [in znova dodelite licenco za Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) za uporabnika, na katerega to vpliva.</span><span class="sxs-lookup"><span data-stu-id="77da5-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="77da5-107">Odprite Officeovo aplikacijo [in se izpišite](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) iz obstoječih uporabniških računov.</span><span class="sxs-lookup"><span data-stu-id="77da5-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="77da5-108">Odprite Nastavitve sistema Windows > **Računi –**& račune in odstranite vse  >  službene račune, razen računa, na katerega to vpliva.</span><span class="sxs-lookup"><span data-stu-id="77da5-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="77da5-109">Odprite Nastavitve sistema Windows > **Računi dostopajo** do službe ali šole in prekinite povezavo z vsemi  >  službeni računi, razen z računom, na katerega to vpliva.</span><span class="sxs-lookup"><span data-stu-id="77da5-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="77da5-110">Ponastavite stanje aktiviranja Officea.</span><span class="sxs-lookup"><span data-stu-id="77da5-110">Reset the Office activation state.</span></span> <span data-ttu-id="77da5-111">[Preberite več o tem.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)</span><span class="sxs-lookup"><span data-stu-id="77da5-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="77da5-112">[Vpišite se](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) s tem uporabniškim računom.</span><span class="sxs-lookup"><span data-stu-id="77da5-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="77da5-113">Če želite dodatne rešitve za odpravljanje težav, glejte [Napake v Officeu, ki nelicencirani izdelek in aktiviranje.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="77da5-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>