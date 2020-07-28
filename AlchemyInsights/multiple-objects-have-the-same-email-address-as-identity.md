---
title: Več predmetov ima enak e-poštni naslov kot identiteta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439710"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="83909-102">Več predmetov ima enak e-poštni naslov kot identiteta</span><span class="sxs-lookup"><span data-stu-id="83909-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="83909-103">**Več predmetov**</span><span class="sxs-lookup"><span data-stu-id="83909-103">**Multiple objects**</span></span>

<span data-ttu-id="83909-104">Eden od pogostih razlogov za to napako je, da ne more pravilno usmerjati zahteve outlookovega spletnega dostopa v prisotnosti več predmetov z istim e-poštnim naslovom kot identiteta.</span><span class="sxs-lookup"><span data-stu-id="83909-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="83909-105">Če želite poiskati te predmete, zaženite te ukaze:</span><span class="sxs-lookup"><span data-stu-id="83909-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="83909-106">· Prejemnika<email address></span><span class="sxs-lookup"><span data-stu-id="83909-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="83909-107">· Pridobitev uporabnika<email address></span><span class="sxs-lookup"><span data-stu-id="83909-107">· Get-User <email address></span></span>

<span data-ttu-id="83909-108">· Pridobitev <email address> uporabnika -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="83909-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="83909-109">· Pokliči stik<email address></span><span class="sxs-lookup"><span data-stu-id="83909-109">· Get-Contact <email address></span></span>

<span data-ttu-id="83909-110">· Get-Mailbox <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="83909-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="83909-111">· Get-Nabiralnik <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="83909-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="83909-112">· Get-Poštni <email address> nabiralnik -NeaktivnoMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="83909-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="83909-113">Če želite odpraviti težavo, odstranite več predmetov z isto e-poštno identiteto in se prepričajte, da obstaja en predmet z določeno e-poštno identiteto in da je njena vrsta prejemnika UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="83909-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="83909-114">**Isti naslov se uporablja za poslovne in potrošniške nabiralnike**</span><span class="sxs-lookup"><span data-stu-id="83909-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="83909-115">Drug vzrok je, ko se isti naslov uporablja za poslovne in potrošniške nabiralnike.</span><span class="sxs-lookup"><span data-stu-id="83909-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="83909-116">v to skrinja, uporabnik morati sprememba svoj primaren potrošnik alias do kavarna zaslomba to lliterarna podlaga dramskega dela.</span><span class="sxs-lookup"><span data-stu-id="83909-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="83909-117">To je trajna napaka, ki ne izgine brez posredovanja.</span><span class="sxs-lookup"><span data-stu-id="83909-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="83909-118">Če želite podrobnosti, [glejte Spreminjanje e-poštnega naslova ali telefonske številke za Microsoftov račun](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="83909-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>