---
title: Dovoljenja za koledar
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
- "3800009"
- "611"
ms.openlocfilehash: 4bf7680a422f096401f0a87bccd1b8dd11f4489f882bcc06864e37d6a248438c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046120"
---
# <a name="calendar-permissions"></a>Dovoljenja za koledar

Uporabniki lahko spremenijo svoja dovoljenja za koledar Outlook uporabniki v spletu ali drugih odjemalcih, vendar boste morali kot skrbnik morda tudi raziskati.  
Z Exchange ukazom »cmdlet« lupine PowerShell prikažete dovoljenje za uporabnikov koledar:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Če želite več informacij, glejte:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Dovoljenja za koledar so uporabljena za skupno rabo koledarjev, za več informacij o skupni rabi koledarja Outlook koledar, si oglejte te članke:

- [Skupna raba koledarja programa Outlook z drugimi osebami](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Skupna raba koledarja v Outlook v spletu za podjetja](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Če želite odpraviti težave z dovoljenjem koledarja, lahko [uporabite pomočnik za podporo in obnovitev](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) koledarja.