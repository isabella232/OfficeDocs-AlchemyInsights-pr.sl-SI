---
title: Nastavite samodejne odgovore za nabiralnik
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
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820950"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="ec3fe-102">Nastavite samodejne odgovore za nabiralnik uporabnika</span><span class="sxs-lookup"><span data-stu-id="ec3fe-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="ec3fe-103">**Način 1**</span><span class="sxs-lookup"><span data-stu-id="ec3fe-103">**Method 1**</span></span>

1. <span data-ttu-id="ec3fe-104">Vpišite se v portal Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ec3fe-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="ec3fe-105">Izberite **Uporabniki > Aktivni uporabniki** (ali **Skupine > Nabiralniki v skupni rabi**, če to nastavljate za nabiralnik v skupni rabi).</span><span class="sxs-lookup"><span data-stu-id="ec3fe-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="ec3fe-106">Izberite uporabnika, ki ima Microsoft Exchangeev nabiralnik.</span><span class="sxs-lookup"><span data-stu-id="ec3fe-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="ec3fe-107">V pojavnem meniju na desni izberite **Nastavitve pošte > Samodejni odgovori** (če gre za nabiralnik v skupni rabi, v pojavnem obvestilu preprosto kliknite **Samodejni odgovori**).</span><span class="sxs-lookup"><span data-stu-id="ec3fe-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="ec3fe-108">**Način 2**</span><span class="sxs-lookup"><span data-stu-id="ec3fe-108">**Method 2**</span></span>

1. <span data-ttu-id="ec3fe-109">Vpišite se v skrbniški portal okolja Microsoft 365 s skrbniškimi poverilnicami.</span><span class="sxs-lookup"><span data-stu-id="ec3fe-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="ec3fe-110">Razširite razdelek **Skrbniška središča** in kliknite **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="ec3fe-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="ec3fe-111">Kliknite sliko v zgornjem desnem kotu, kliknite **Drug uporabnik**, nato pa izberite uporabniški nabiralnik, ki ga želite spremeniti.</span><span class="sxs-lookup"><span data-stu-id="ec3fe-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="ec3fe-112">Na levi strani izberite **Možnosti**, kliknite **Organiziraj e-pošto**, nato pa kliknite **Samodejni odgovori.**</span><span class="sxs-lookup"><span data-stu-id="ec3fe-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="ec3fe-113">**Način 3**</span><span class="sxs-lookup"><span data-stu-id="ec3fe-113">**Method 3**</span></span>

<span data-ttu-id="ec3fe-114">Zaženite ta pripomoček »cmdlet« v storitvi Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="ec3fe-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="ec3fe-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="ec3fe-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="ec3fe-116">Če želite več informacij o tem pripomočku »cmdlet«, glejte [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="ec3fe-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
