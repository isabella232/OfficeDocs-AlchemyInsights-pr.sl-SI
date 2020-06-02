---
title: 1336 RecoverableItems mapa je polna
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510768"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="74312-102">Mapa» Obnovljivo «je polna</span><span class="sxs-lookup"><span data-stu-id="74312-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="74312-103">Za nabiralnike Exchange Online je privzeta omejitev shranjevanja za mapo» Obnovljivo «30 GB.</span><span class="sxs-lookup"><span data-stu-id="74312-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="74312-104">Omejitev shranjevanja za mapo» Obnovljivo «se samodejno poveča na 100 GB, če je nabiralnik postavljen na čakanje zaradi spora, zadržanje e-odkrivanja ali pa je dodeljen pravilniku o hranjenju.</span><span class="sxs-lookup"><span data-stu-id="74312-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="74312-105">Ko mapa» Obnovljivo «doseže omejitev shranjevanja, je funkcija nabiralnika prizadeta na naslednje načine:</span><span class="sxs-lookup"><span data-stu-id="74312-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="74312-106">Uporabnik ne more izbrisati elementov iz nabiralnika.</span><span class="sxs-lookup"><span data-stu-id="74312-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="74312-107">Pomočnik za upravljane mape ne more izbrisati elementov, ki temeljijo na oznaki za hranjenje ali v nastavitvah upravljane mape.</span><span class="sxs-lookup"><span data-stu-id="74312-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="74312-108">Za nabiralnike, ki imajo omogočeno Obnovitev posameznega artikla ali so dani na voljo, postopek zaščite strani za kopiranje na pisanje ne more vzdrževati različic elementov, ki jih je uredil uporabnik.</span><span class="sxs-lookup"><span data-stu-id="74312-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="74312-109">Za nabiralnike, ki imajo omogočeno beleženje dnevnika revizij nabiralnika, ni mogoče shraniti vnosov dnevnika revizij nabiralnika v podmapo revizijah v mapi» obnovljivo «.</span><span class="sxs-lookup"><span data-stu-id="74312-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="74312-110">Za nabiralnike, ki niso na voljo, lahko skrbniki s pomočjo `Search-Mailbox -SearchDumpsterOnly -DeleteContent` ukaza v PowerShell Exchange Online izbrišejo elemente v mapi» obnovljivo «.</span><span class="sxs-lookup"><span data-stu-id="74312-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="74312-111">Če želite več informacij, glejte naslednje teme:</span><span class="sxs-lookup"><span data-stu-id="74312-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="74312-112">Iskanje in brisanje sporočil</span><span class="sxs-lookup"><span data-stu-id="74312-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="74312-113">Iskalni nabiralnik</span><span class="sxs-lookup"><span data-stu-id="74312-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="74312-114">Za nabiralnike, ki so na zadržani, morajo skrbniki odstraniti zadržko, preden lahko izbrišejo elemente iz mape» Obnovljivo «.</span><span class="sxs-lookup"><span data-stu-id="74312-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="74312-115">Če želite več informacij, glejte [brisanje elementov v mapi» obnovljivo «v nabiralnikih v oblaku, ki jih držite](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="74312-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="74312-116">Če želite preprečiti, da bi mapa» Obnovljivo «postala polna, lahko skrbniki povečajo omejitev shranjevanja mape» Obnovljivo «za nabiralnike na zadržanju in nastavijo pravilnik o hranjenju nabiralnika, ki premakne elemente iz mape» Obnovljivo «v arhivski nabiralnik uporabnika.</span><span class="sxs-lookup"><span data-stu-id="74312-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="74312-117">Glejte [povečanje kvote za obnovljivo postavko za nabiralnike na zadržanju](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="74312-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
