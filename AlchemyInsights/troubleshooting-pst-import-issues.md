---
title: Odpravljanje težav pri uvozu PST
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059831"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="d485b-102">Odpravljanje težav pri uvozu PST</span><span class="sxs-lookup"><span data-stu-id="d485b-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="d485b-103">Če uvažate znotraj odjemalca za Outlook, glejte Odpravljanje težav [pri uvozu Outlookove datoteke .pst.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)</span><span class="sxs-lookup"><span data-stu-id="d485b-103">If you are importing within the Outlook client itself, see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="d485b-104">Če uporabljate storitev uvoza in je obstala, upoštevajte, da vsaka datoteka PST, ki jo prenesete na mesto shrambe Azure, ne sme biti večja od 20 GB.</span><span class="sxs-lookup"><span data-stu-id="d485b-104">If you are using Import Service and it's stuck, note that each PST file that you upload to the Azure Storage location should be no larger than 20GB.</span></span> <span data-ttu-id="d485b-105">Datoteke PST, večje od 20 GB, lahko vplivajo na učinkovitost postopka uvoza datoteke PST.</span><span class="sxs-lookup"><span data-stu-id="d485b-105">PST files larger than 20GB may impact the performance of the PST import process.</span></span> <span data-ttu-id="d485b-106">Če želite več informacij o odpravljanju težav z obtičimi posli, glejte [Težave, ki vplivajo na opravila uvoza datotek PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="d485b-106">For more information troubleshooting stuck jobs, see [Issues that affect PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

- <span data-ttu-id="d485b-107">Če želite preveriti stanje določenega posla uvoza, uporabite [Get-MailboxImportRequest -batchname.](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)</span><span class="sxs-lookup"><span data-stu-id="d485b-107">If you want to verify the status of a specific Import job, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="d485b-108">Če si želite ogledati vse podrobnosti storitve uvoza, glejte [Pregled uvažanja datotek PST organizacije.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="d485b-108">For full details on the import service, see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
