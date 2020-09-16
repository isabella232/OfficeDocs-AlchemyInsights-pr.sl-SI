---
title: Zamude pri prejemanju SharePointovih in OneDrive opozoril
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727259"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="68aa4-102">Zamude pri prejemanju SharePointovih in OneDrive opozoril</span><span class="sxs-lookup"><span data-stu-id="68aa4-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="68aa4-103">Najprej preverite mapo» Neželena ali neželena pošta «v e-poštnem sporočilu.</span><span class="sxs-lookup"><span data-stu-id="68aa4-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="68aa4-104">Če **so vsa opozorila iz več datotek ali knjižnic odložena**, obiščite [nadzorno ploščo za zdravstveno stanje](https://portal.office.com/adminportal/home?ref=/servicehealth) , da preverite morebitne svetovalce/incidente, ki se lahko pojavijo v SharePointu ali storitvi Exchange.</span><span class="sxs-lookup"><span data-stu-id="68aa4-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="68aa4-105">Težava je morda v storitvi SharePoint Alert capability ali zamude v e-poštnih sporočilih prek Exchangea.</span><span class="sxs-lookup"><span data-stu-id="68aa4-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="68aa4-106">Upoštevajte tudi, ali je druga e-pošta dostavljena – če ne, je težava verjetno pri deviznih zamudah.</span><span class="sxs-lookup"><span data-stu-id="68aa4-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="68aa4-107">Če **individualna opozorila iz določene datoteke ali knjižnice niso dostavljena**, jo poskusite izbrisati in znova ustvariti.</span><span class="sxs-lookup"><span data-stu-id="68aa4-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="68aa4-108">Če želite znova ustvariti opozorilo [, glejte upravljanje, ogled ali brisanje SharePointovih opozoril](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .</span><span class="sxs-lookup"><span data-stu-id="68aa4-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="68aa4-109">Opozoril ni mogoče poslati v skupino prejemnikov.</span><span class="sxs-lookup"><span data-stu-id="68aa4-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="68aa4-110">Podprte so le varnostne in O365 skupine.</span><span class="sxs-lookup"><span data-stu-id="68aa4-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="68aa4-111">E-poštnih predlog za opozorila ne morete prilagoditi.</span><span class="sxs-lookup"><span data-stu-id="68aa4-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="68aa4-112">Če želite doseči te storitve, morate uporabiti Microsoft Flow ali potek dela za SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="68aa4-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
