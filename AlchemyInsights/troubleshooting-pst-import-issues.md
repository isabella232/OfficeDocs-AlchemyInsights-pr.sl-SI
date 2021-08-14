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
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972435"
---
# <a name="troubleshooting-pst-import-issues"></a>Odpravljanje težav pri uvozu PST

- Če uvažate znotraj odjemalca Outlook, glejte Odpravljanje težav [pri uvozu datoteke .pst Outlook .](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)

- Če uporabljate storitev uvoza in je obstala, upoštevajte, da vsaka datoteka PST, ki jo prenesete na mesto shrambe Azure, ne sme biti večja od 20 GB. Datoteke PST, večje od 20 GB, lahko vplivajo na učinkovitost postopka uvoza datoteke PST. Če želite več informacij o odpravljanju težav z obtičimi posli, glejte [Težave, ki vplivajo na opravila uvoza datotek PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

- Če želite preveriti stanje določenega posla uvoza, uporabite [Get-MailboxImportRequest -batchname.](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)

- Če si želite ogledati vse podrobnosti storitve uvoza, glejte [Pregled uvažanja datotek PST organizacije.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
