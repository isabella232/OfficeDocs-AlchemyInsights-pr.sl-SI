---
title: Omogočanje Microsoftovega zagovornika za Office 365 za SharePoint online, OneDrive in Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747740"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="14c48-102">Omogočanje Microsoftovega zagovornika za Office 365 za SharePoint online, OneDrive in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="14c48-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="14c48-103">S splošnimi skrbniškimi poverilnicami ali varnostnim skrbnikom se prijavite v [središče za varnost in skladnost s predpisi sistema Office 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="14c48-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="14c48-104">V levem podoknu izberite **upravljanje grožnje** in nato izberite   >  [varne Priloge](https://protection.office.com/safeattachment)pravilnika.</span><span class="sxs-lookup"><span data-stu-id="14c48-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="14c48-105">Izberite **Vklopi Microsoft Defender za Office 365 za SharePoint, OneDrive in Microsoft Teams** in nato izberite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="14c48-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="14c48-106">Kot globalni skrbnik ali skrbnik SharePoint Onlinea zaženite ta ukaz» cmdlet «PowerShell s parametrom» **DisallowInfectedFileDownload** «, nastavljenim na» *True*«: [set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="14c48-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="14c48-107">Nastavitev opozoril za zaznane datoteke</span><span class="sxs-lookup"><span data-stu-id="14c48-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="14c48-108">Če želite več informacij, glejte [Microsoft Defender za Office 365 za SharePoint, OneDrive in Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span><span class="sxs-lookup"><span data-stu-id="14c48-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
