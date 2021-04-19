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
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826179"
---
# <a name="troubleshooting-pst-import-issues"></a>Odpravljanje težav pri uvozu PST

- Če uvažate v Outlookovem odjemalcu, glejte [odpravljanje težav z uvažanjem Outlookove datoteke. pst](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Če uporabljate storitev Import in je obtičala, upoštevajte, da ne bi smela biti vsaka datoteka PST, ki jo prenesete na mesto za shranjevanje v storitvi Azure, večja od 20 GB. Datoteke PST, večje od 20 GB, lahko vplivajo na učinkovitost postopka uvoza PST.

- Če želite preveriti stanje določenega uvoza, lahko uporabite [Get-MailboxImportRequest-batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Če želite podrobnejše informacije o storitvi uvoza, si oglejte [pregled uvoza datotek PST v vaši organizaciji](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
