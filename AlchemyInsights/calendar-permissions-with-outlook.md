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
# <a name="calendar-permissions"></a><span data-ttu-id="64f8d-102">Dovoljenja koledarja</span><span class="sxs-lookup"><span data-stu-id="64f8d-102">Calendar Permissions</span></span>

<span data-ttu-id="64f8d-103">Uporabnik moči sprememba svoj lasten koledar dovoljenje s razgled naprej ujeti ali drugi varovanci, šele kot a pomoč vi maj potreba v preiskovati enako.</span><span class="sxs-lookup"><span data-stu-id="64f8d-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="64f8d-104">Z ukazom» cmdlet «Exchange PowerShell vam bo v uporabnikovem koledarju pokazal dovoljenje:</span><span class="sxs-lookup"><span data-stu-id="64f8d-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="64f8d-105">Če si želite ogledati več informacij, glejte naslednje:</span><span class="sxs-lookup"><span data-stu-id="64f8d-105">To see more information see the following:</span></span>

- [<span data-ttu-id="64f8d-106">Get-Mailboxfolderdovoljenje</span><span class="sxs-lookup"><span data-stu-id="64f8d-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="64f8d-107">Set-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="64f8d-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="64f8d-108">Dodaj-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="64f8d-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="64f8d-109">Dovoljenja koledarja se uporabljajo pri skupni rabi koledarjev, če si želite ogledati več informacij o skupni rabi Outlookovega koledarja, glejte te članke:</span><span class="sxs-lookup"><span data-stu-id="64f8d-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="64f8d-110">Skupna raba koledarja programa Outlook z drugimi osebami</span><span class="sxs-lookup"><span data-stu-id="64f8d-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="64f8d-111">Delite svoj koledar v Outlooku v spletu za podjetja</span><span class="sxs-lookup"><span data-stu-id="64f8d-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="64f8d-112">Če želite odpraviti dovoljenje za koledar, lahko uporabite orodje [pomočnika za podporo in obnovitev](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .</span><span class="sxs-lookup"><span data-stu-id="64f8d-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>