---
title: Dovoljenja za koledar
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
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748809"
---
# <a name="calendar-permissions"></a>Dovoljenja za koledar

Uporabniki lahko sami spreminjajo dovoljenja za koledar z Outlookom v spletu ali drugimi odjemalci, temveč tudi kot skrbnik, ki ga boste morda morali raziskovati.  
Z ukazom» cmdlet «za Exchange PowerShell bo na uporabnikovem koledarju prikazano dovoljenje:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Če si želite ogledati več informacij, glejte to:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Dovoljenja za koledar se uporabljajo v skupni rabi koledarjev, če si želite ogledati več informacij o skupni rabi koledarja Outlooka, si oglejte te članke:

- [Skupna raba koledarja programa Outlook z drugimi osebami](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Skupna raba koledarja v Outlooku v spletu za podjetja](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Če želite odpraviti težave z dovoljenjem koledarja, lahko uporabite orodje [pomočnik za podporo in obnovitev](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .