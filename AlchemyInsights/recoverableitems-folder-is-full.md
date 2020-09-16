---
title: Mapa» 1336 RecoverableItems «je polna
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741283"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="7dc7e-102">Mapa» obnovljivi elementi «je polna</span><span class="sxs-lookup"><span data-stu-id="7dc7e-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="7dc7e-103">Za nabiralnike v storitvi Exchange Online je privzeta omejitev shrambe za mapo» obnovljivi elementi «30 GB.</span><span class="sxs-lookup"><span data-stu-id="7dc7e-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="7dc7e-104">Omejitev shrambe za mapo» obnovljivi elementi «je samodejno povečana na 100 GB, če je nabiralnik nastavljen na zadržanje zaradi spora, E-odkrivanje zadržanje ali pa je dodeljen pravilniku o hranjenju.</span><span class="sxs-lookup"><span data-stu-id="7dc7e-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="7dc7e-105">Ko mapa» obnovljivi elementi «doseže omejitev shrambe, vpliva na funkcije nabiralnika na te načine:</span><span class="sxs-lookup"><span data-stu-id="7dc7e-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="7dc7e-106">Uporabnik ne more izbrisati elementov iz nabiralnika.</span><span class="sxs-lookup"><span data-stu-id="7dc7e-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="7dc7e-107">Pomočnik za upravljane mape ne more izbrisati elementov, ki temeljijo na nastavitvah oznake hranjenja ali upravljanih map.</span><span class="sxs-lookup"><span data-stu-id="7dc7e-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="7dc7e-108">Za nabiralnike, ki imajo omogočeno obnovitev enega elementa ali pa so zadržane, proces zaščite pred kopiranjem na mesto pisanja ne more vzdrževati različic elementov, ki jih je uredil uporabnik.</span><span class="sxs-lookup"><span data-stu-id="7dc7e-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="7dc7e-109">Za nabiralnike, ki imajo omogočeno pisanje dnevnika nadzora nabiralnika, ni mogoče shraniti vnosov dnevnika nadzora nabiralnika v podmapo» revizije «v mapi» obnovljivi elementi «.</span><span class="sxs-lookup"><span data-stu-id="7dc7e-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="7dc7e-110">Za nabiralnike, ki niso zadržani, lahko skrbniki z `Search-Mailbox -SearchDumpsterOnly -DeleteContent` ukazom PowerShell za Exchange Online izbrišejo elemente v mapi» obnovljivi elementi «.</span><span class="sxs-lookup"><span data-stu-id="7dc7e-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="7dc7e-111">Če želite več informacij, glejte te teme:</span><span class="sxs-lookup"><span data-stu-id="7dc7e-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="7dc7e-112">Iskanje in brisanje sporočil</span><span class="sxs-lookup"><span data-stu-id="7dc7e-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="7dc7e-113">Iskanje nabiralnika</span><span class="sxs-lookup"><span data-stu-id="7dc7e-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="7dc7e-114">Za nabiralnike, ki so zadržani, morajo skrbniki odstraniti zadržanje, preden lahko izbrišejo elemente iz mape» obnovljivi elementi «.</span><span class="sxs-lookup"><span data-stu-id="7dc7e-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="7dc7e-115">Če želite več informacij, glejte [brisanje elementov v mapi» obnovljivi elementi «nabiralnikov v oblaku v zadržanju](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="7dc7e-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="7dc7e-116">Če želite preprečiti, da bi se mapa» obnovljivi elementi «ohranila v celoti, lahko skrbniki povečajo omejitev shrambe mape» obnovljivi elementi «za nabiralnike v zadržanju in nastavijo pravilnik o hranjenju nabiralnika, ki premakne elemente iz mape» obnovljivi elementi «v nabiralnik uporabnikovega arhiva.</span><span class="sxs-lookup"><span data-stu-id="7dc7e-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="7dc7e-117">Glejte [povečanje kvote za obnovljive elemente za nabiralnike v zadržanju](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="7dc7e-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
