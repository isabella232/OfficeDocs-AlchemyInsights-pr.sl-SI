---
title: Dovoljenja koledarja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862167"
---
# <a name="calendar-permissions"></a>Dovoljenja koledarja

Uporabnik moči sprememba svoj lasten koledar dovoljenje s razgled naprej ujeti ali drugi varovanci, šele kot a pomoč vi maj potreba v preiskovati enako.  
Z ukazom» cmdlet «Exchange PowerShell vam bo v uporabnikovem koledarju pokazal dovoljenje:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Če si želite ogledati več informacij, glejte naslednje:

- [Get-Mailboxfolderdovoljenje](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Dodaj-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Dovoljenja koledarja se uporabljajo pri skupni rabi koledarjev, če si želite ogledati več informacij o skupni rabi Outlookovega koledarja, glejte te članke:

- [Skupna raba koledarja programa Outlook z drugimi osebami](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Delite svoj koledar v Outlooku v spletu za podjetja](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Če želite odpraviti dovoljenje za koledar, lahko uporabite orodje [pomočnika za podporo in obnovitev](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .